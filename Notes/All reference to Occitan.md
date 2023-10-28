---
aliases:
---
%%
topic:: [[Occitan]]
related:: 
created:: October 22, 2023
last edit:: `$= moment(dv.current().file.mtime.toString()).format("YYYY-MM-DD")`
type:: query
action:: false
%%
## All References
```dataviewjs
const pagesWithTopic = await Promise.all(
    dv
    .pages()
    .map(n => new Promise(async (resolve, reject) => {
        const content = await dv.io.load(n.file.path);
        resolve({
            link: n.file.link,
            content
        });
    }))
);

const topicsByPage = pagesWithTopic.map(({
    link,
    content
}) => ({
    link,
    content: content
	    .split('\n\n')
        .filter(content => content.includes('Occitan'))
        .filter(content => !content.includes('topic:: [[Occitan]]'))

}));

topicsByPage.forEach(
    page =>
    page.content.forEach(
        n => dv.paragraph(`${n} (${page.link})`)
    )
);
```

# Reference





