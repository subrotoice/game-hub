## Chakra Grid[Chakra Grid:](https://chakra-ui.com/docs/components/grid)

** Basic Chakra and Responsiveness **

```javascript
<Grid templateAreas={`"nav nav" "aside main"`}>
  <GridItem bg="pink.300" area="nav">
    Nav
  </GridItem>
  <GridItem bg="yellow.300" area="aside">
    Aside
  </GridItem>
  <GridItem bg="green.300" area="main">
    Main
  </GridItem>
</Grid>

// Responsive Component
<Grid
    templateAreas={{
    base: `"nav" "main"`,
    lg: `"nav nav" "aside main"`,
    }}
>
    <GridItem bg="pink.300" area="nav">
    Nav
    </GridItem>
    <Show above="lg">
    <GridItem bg="yellow.300" area="aside">
        Aside
    </GridItem>
    </Show>
    <GridItem bg="green.300" area="main">
    Main
    </GridItem>
</Grid>

// Logo and Hstack in chakrqa
<Grid
    templateAreas={{
    base: `"nav" "main"`,
    lg: `"nav nav" "aside main"`,
    }}
>
    <GridItem area="nav">
    <NavBar />
    </GridItem>
    <Show above="lg">
    <GridItem bg="yellow.300" area="aside">
        Aside
    </GridItem>
    </Show>
    <GridItem bg="green.300" area="main">
    Main
    </GridItem>
</Grid>
// NavBar.tsx
<HStack>
    <Image src={logo} boxSize="60px" />
    <Text>NavBar</Text>
</HStack>
```
