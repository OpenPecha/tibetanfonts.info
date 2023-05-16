
# Working with Flowbite Pro

1. The Flowbite Pro Figma designs are copied into OpenPecha's Figma account. 
2. One designer/frontend developer manages the Figma Flowbite.
3. Assemble any new UI view for a web application in Figma using Flowbite Figma components.
4. Customize the styling for each component in Figma to fit the palette/theme of the organization and/or the particular web application.
5. The frontend developer extracts the required information, like CSS properties, positioning, and sizing of components, etc., from each completed UI view in Figma.
6. Import Flowbite Pro into the Vue3 frontend code using the CDN (JS script embed) method. (We'll import using Flowbite-Vue once it works for all Flowbite components.)
7. If needed, use Flowbite v1.5.0 for compatibility, like how we use LTS versions. 
8. Wrap Flowbite JS components into Vue3 components or use them directly, depending on the reusability factor.
9. Customize styling using Tailwind classes or directly with CSS props.
 
To take full advantage of Flowbite Pro with Vue, you need to follow steps five through nine.