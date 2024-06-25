# Darya Korbut


## Contacts

* **Address:** Belarus, Minsk
* **Phone:** +375-29-599-63-42
* **Email:** dashkakorbut@gmail.com
* **Links:**
  * [Telegram](https://t.me/Darya0322)
  * [LinkedIn](https://www.linkedin.com/in/darya-korbut-96a6461b7/)
  * [GitHub](https://github.com/Dasha2203)

## About me

I graduated Minsk Radio-Technical College that's where I learned the basics of programming. After then I gratuated Belarusian State University of Informatics and Radioelectronics in 2024.

During my studies, I did some freelance work. I developed web-pages using **HTML, CSS, JS, BEM**.
A developed PWA applications using **React, React Router, React context, WebSocket, styled-components.**

**_The list of tasks I've been doing_**

* Lendings development **(HTML, CSS, JS, SASS, BEM, SMARTY)**
* SPA development **(React, React Router, styled components, React context)**
* Optimizing the display of a large list of data using a virtualized list
* Optimize page load speed
* Forms development and validation
* Synchronization of data with other sites on the server side

I am currently working for a client and they are developing an information project using **Next.js, Tailwind.css, GraphQL**. I work with a lot of data, display them in tables with pagination. I develop filters and data search on the site.

I love website development as I enjoy working not only with the functional part but also the look and feel of the website. I like layout and logic development. I have not had a mentor, but I try to develop on my own, periodically revise my code and make edits. 

I want to learn new technologies, pump up my skills and develop more complex functionality.

I also watch videos on YouTube and listen to podcasts.

## Skills

* **Basic:** HTML, CSS, JS (Sass, Jquery, BEM, REST)
* Smarty
* React (React router, Redux, React context, hooks)
* Next.js
* The foundation of Node.js and Nest.js
* Styled-components, Tailwind.css, Material UI, Bootstrap
* Git, figma, Rest API, GraphQL, OOP


## Code examples

Preparation of sections for displaying in a convenient form of Sitemap page

```typescript
  const sitemapItems: {
    category: string
    label: string
    url: string
  }[] = [
    ...articles.map((it) => ({
      category: 'articles',
      label:
        it.translations?.find((it) => it.locale === locale)?.title ?? it.title,
      url: getUrl(`/blog/${it.slug}`),
    })),
    ...exchanges.map((it) => ({
      category: 'exchanges',
      label: t('exchange:title', { name: it.name }).replace(' | Criffy', ''),
      url: getUrl(`/exchanges/${it.slug}`),
    })),
    ...wallets.map((it) => ({
      category: 'wallets',
      label: t('wallet:title', { name: it.name }).replace(' | Criffy', ''),
      url: getUrl(`/wallets/${it.slug}`),
    })),
    ...currencies.map((it) => ({
      category: 'cryptocurrencies',
      label: t('currency:title', { name: it.name, symbol: it.symbol }).replace(
        ' | Criffy',
        '',
      ),
      url: getUrl(`/currencies/${it.slug}`),
    })),
    ...fiats.map((it) => ({
      category: 'fiat',
      label: t('fiat:title', { name: it.name, symbol: it.symbol }).replace(
        ' | Criffy',
        '',
      ),
      url: getUrl(`/currencies/${it.slug}`),
    })),
  ]
```

Task from [LeetCode](https://leetcode.com/)

```typescript
type CacheType = {
    [key: string]: number
}

function twoSum(nums: number[], target: number): number[] {
    const cache: CacheType = {}

    for (let i = 0; i < nums.length; i++) {
        let num = target - nums[i]

        if (cache[num] !== undefined) return [cache[num], i] 

        cache[nums[i]] = i
    }

    return []
};
```
