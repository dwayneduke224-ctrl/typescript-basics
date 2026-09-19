1. What was the biggest advantage you noticed when using TypeScript vs. plain JavaScript?
2. Describe a specific error TypeScript caught that JavaScript would have missed.
3. What is the difference between an interface and a type alias in TypeScript? When would you use each?
4. Why do we use `export` and `import` in TypeScript files?
5. What happens to interfaces when TypeScript compiles to JavaScript? Why?
6. If you had to add a `Review` entity (users reviewing products), what would its interface look like? Write it out.

ANSWERS
1.The biggest advantage I noticed is that TypeScript can check my code for errors before running it. It also helps me with autocomplete and tells me what type of data I should use.
2. const badUserId: number = "not-a-number";
3. An interface is used to describe the structure of an object. In my project, I used interfaces for User and Product.
4. We use export so we can use functions or interfaces from another file. We use import to bring them into the file we are working on.
5. The interfaces are removed when TypeScript is compiled into JavaScript. They are only used by TypeScript to check our code while developing. JavaScript does not need the interfaces when the program runs.
6. export interface Review {
    id: number;
    userId: number;
    productId: number;
    rating: number;
    comment: string;
    createdAt: Date;
}
