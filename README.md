# jetstone
A new 24x24 Dwarf Fortress Tileset and raw files.  Now that retina screens are a thing, we have the option to have slightly nicer tiles for use in playing dwarf fortress.  Further, as of mid-2016, it doesn't seem like most of the tileset makers are keeping up with compatibility.  So, here's a new one.

If you intend to fork or contribute to this project, be aware of the following link, as it helps a great deal in assessing what to do with each tile within the limits we have set upon us.

http://dwarffortresswiki.org/DF2014:Tilesets

## Task List 1st Release Candidate

- [x] Establish Text/Font Tiles
- [ ] Design Mineralization Tiles
- [ ] Assign Mineralization Raws to Tiles
- [ ] Design Constructions
- [ ] Assign Construction Raws/Init to Tiles
- [ ] Design Furniture
- [ ] Assign Furniture Raws to Tiles
- [ ] Design Flora
- [ ] Assign Flora Raws to Tiles
- [ ] Design Trinkets, Tools and Doodads
- [ ] Assign Trinket, Tool and Doodad Raws to Tiles

## Rocks and Minerals

See: https://en.wikipedia.org/wiki/Crystal_habit for typical mineral shapes
See: https://en.wikipedia.org/wiki/Rock_(geology) for typical rock types and textures

### Tile Choices

* 134 - Mostly Igneous Intrusive Rock; **Large Obvious Grains**
* 135 - Mostly Igneous Extrusive Rock; **Small to Invisible Grains**
* 136 - Mostly Metamorphic Rock; **Distorted Bands or Squished Blotches**
* 137 - Mostly Sedimentary Rock; **Layers or Lines, Subtle or Strong**

* 139 - Mostly Minerals; **Rounded forms**
* 140 - Mostly Minerals; **Columnar facets**
* 141 - Mostly Minerals; **Veins**
* 142 - Mostly Minerals; **Striations or Platings**

* 169 - Mostly Gems; **Triangular Facets**
* 170 - Mostly Gems; **Square Facets**
* 171 - Mostly Gems; **Hexagonal Facets**
* 172 - Mostly Gems; **Monoclinic Facets** 

### inorganic_stone_layer

| Type | Subtype | Name | Habit | Colors | Tile |
| --- | --- | --- | --- | --- | --- |
| rock | sedimentary | **SANDSTONE** | subtle layering or striations | light warm tones | 137 |
| rock | sedimentary | **SILTSTONE** | little to no texture | light warm tones | 135 | 
| rock | sedimentary | **MUDSTONE** | little to no texture | middle warm greys | 135 |
| rock | sedimentary | **SHALE** | subtle layering only | dark greys | 137 |
| rock | sedimentary | **CLAYSTONE** | distinct layers | dark greys and browns | 137 |
| rock | sedimentary | **ROCK_SALT**<sup>1</sup> | cubic crystallization | white to light pink | 140 |
| rock | sedimentary | **LIMESTONE** | largely uniform texture | white to cream | 135 |
| rock | sedimentary | **CONGLOMERATE** | large random inclusions in matrix | dark with bright spots | 134 |
| rock | sedimentary | **DOLOMITE**<sup>2</sup> | fairly uniform grainy texture | middle grey to warm grey | 135 |
| rock | sedimentary | **CHERT** | subtle striations | brownish red | 137 |
| rock | sedimentary | **CHALK** | little to no texture | bright white | 135 |
| rock | igneous intrusive | **GRANITE**<sup>3</sup> | heavy spotted textures | white, black, cream | 134 |
| rock | igneous intrusive | **DIORITE** | large grains | light with dark grains | 134 |
| rock | igneous intrusive | **GABBRO** | large grains | dark with some light grains | 134 |
| rock | igneous extrusive | **RHYOLITE** | fairly uniform with small grains | light grey to warm tones | 135 |
| rock | igneous extrusive | **BASALT**  | fairly uniform texture | dark grey to black | 135 |
| rock | igneous extrusive | **ANDESITE** | somewhat uniform with bright specks | middle grey | 135 |
| rock | igneous extrusive | **DACITE** | uniform except for bright specks | light grey | 135 |
| rock | igneous extrusive | **OBSIDIAN** | lustrous and uniform, rare banding | black, red bands | 139 |
| rock | metamorphic | **QUARTZITE** | subtle mottling or bands | reddish cream to white | 135 |
| rock | metamorphic | **SLATE** | subtle lines or uniform | dark grey | 137 |
| rock | metamorphic | **PHYLLITE** | subtle undulating waves | warm light greys | 136 |
| rock | metamorphic | **SCHIST**<sup>4</sup> | grainy, mottled, flowing | middle grey | 136 |
| rock | metamorphic | **GNEISS** | strong wavy or jagged banding | dark gray with bright bands | 136 |
| rock | metamorphic | **MARBLE**<sup>5</sup> | subtle to strong dark bands in light material | white to cream | 136 |

### inorganic_stone_mineral

| Type | Subtype | Name | Habit | Colors | Tile |
| --- | --- | --- | --- | --- | --- |
| mineral | oxide | **HEMATITE** | angular and faceted | black, brown, red | 169 |
| mineral | hydroxide | **LIMONITE** | blotchy, amorphous | yellow to red | 134 |
| mineral | N/A | **GARNIERITE**<sup>6</sup> | blotchy, amorphous | greens | 134 |
| element | metal | **NATIVE_GOLD** | fans, veins, plates | bright yellow | 141 |
| element | metal | **NATIVE_SILVER** | fans, veins, plates | bright white | 141 |
| element | metal | **NATIVE_COPPER** | fans, veins, plates | brown to red | 141 |
| mineral | hydroxide | **MALACHITE** | bulbous sheets of tiny crystals | dark green | 139 |
| mineral | sulfide | **GALENA** | cubic and lustrous | dark grey | 170 |
| mineral | sulfide | **SPHALERITE** | triangular lustrous facets | dark grey, rarely red | 169 |
| mineral | oxide | **CASSITERITE** | lustrous and triangular | black to mid grey | 169 |
| rock | metamorphic | **COAL_BITUMINOUS**<sup>7</sup> | sometimes lustrous but low texture | black | 135 |
| rock | metamorphic | **LIGNITE** | dull and with little texture | dark brown | 135 |
| element | metal | **NATIVE_PLATINUM** | fans, veins, plates | light grey | 141 |
| mineral | sulfide | **CINNABAR** | grainy; triangular facets at best | dark red | 169 |
| mineral | sulfide | **COBALTITE** | confused cubic faces | dark grey or ruddy brown | 170 |
| mineral | sulfosalt | **TETRAHEDRITE** | reflective triangular faces | dark yellow to grey | 169 |
| mineral | chloride | **HORN_SILVER** | grainy texture with little structure | dark yellow to grey | 135 |
| mineral | sulfate | **GYPSUM** | angular striations and long crystals | white | 172 |
| mineral | silicate | **TALC** | little texture or structure | white to yellow | 135 |
| rock | metamorphic | **JET**<sup>8</sup> | little texture, subtle striations | black | 137 |
| rock | sedimentary | **PUDDINGSTONE** | uniform midtone with bright blotches | reds, browns | 134 |
| rock | metamorphic | **PETRIFIED_WOOD** | strong radiating bands | reds, browns, some whites | 136 |
| element | semimetal | **GRAPHITE** | lustrous with occasional faceting | black | 171 |
| element | nonmetal | **BRIMSTONE**<sup>9</sup> | chalky and indistinct | bright yellow | 135 |
| rock | igneous intrusive | **KIMBERLITE** | grainy uniform with occasional specks | mid to dark grey | 134 |
| mineral | sulfide | **BISMUTHINITE** | fibrous striations at best | dark grey | 142 |
| mineral | sulfide | **REALGAR** | semitranslucent with sharp edges | bright red | 172 |
| mineral | sulfide | **ORPIMENT** | small crystals or blades | orange to red | 142 |
| mineral | sulfide | **STIBNITE** | lustrous lined columns | mid grey | 142 |
| mineral | sulfide | **MARCASITE** | lustrous plates and wedges | brownish grey | 142 |
| mineral | chloride | **SYLVITE** | little texture or structure | creams to reds | 135 |
| mineral | halide | **CRYOLITE** | little texture or structure | white | 135 |
| mineral | oxide | **PERICLASE** | blotchy and indistict | speckled light greys | 134 |
| mineral | oxide | **ILMENITE** | rough and angular | black or dark brown | 169 |
| mineral | oxide | **RUTILE** | crystallite or hairy | deep red to purple to yellow | 142 |
| mineral | oxide | **MAGNETITE** | low lustre with sharp angles | black or dark brown | 169 |
| mineral | oxide | **CHROMITE** | mottled and indistinct | dark grey with highlights | 134 |
| mineral | oxide | **PYROLUSITE** | shiny spheroid bulbs | black to bluish black | 139 |
| mineral | oxide | **PITCHBLENDE** | occasional facets; usually rounded | brownish black | 139 |
| rock | sedimentary | **BAUXITE** | mixture of light matrix and dark blots | light grey and brown | 134 |
| element | metal | **NATIVE_ALUMINUM** | fans, veins, plates | light grey | 141 |
| mineral | borate | **BORAX** | usually massive, rare crystal structures | white | 135 |
| mineral | silicate | **OLIVINE**<sup>10</sup> | glassy, usually amorphous, bubbly | dark to light green | 139 |
| mineral | silicate | **HORNBLENDE**<sup>11</sup> | rough and shapeless | black with rare specks | 135 |
| mineral | silicate | **KAOLINITE** | layered microcrystals | white to dark cream | 137 |
| mineral | silicate | **SERPENTINE**<sub>12<sup> | untextured to layered | dark green | 136 |
| mineral | silicate | **ORTHOCLASE** | often amorphous, can have angular crystals | cream to yellow | 172 |
| mineral | silicate | **MICROCLINE** | often amorphous, can have anuglar crystals | bright green or blue | 172 |
| mineral | silicate | **MICA** | in stacked sheets or crushed | silver, purple, or blackish | 142 |
| mineral | carbonate | **CALCITE** | amorphous or with pointed crystals | white to orange | 169 |
| mineral | nitrate | **SALTPETER** | amorphous with little texture | white | 135 |
| mineral | carbonate | **ALABASTER**<sup>13</sup> | little texture | white to dark cream | 135 |
| mineral | sulfate | **SELENITE**<sup>14</sup> | monoclinic angles or amorphous | white to dark cream | 172 |
| mineral | sulfate | **SATINSPAR**<sup>14</sup> | plated or feathered | milky white | 142 |
| mineral | sulfate | **ANHYDRITE** | plated or fibrous | white | 142 |
| mineral | sulfate | **ALUNITE** | fibrous or amorphous | dark cream to orange | 142 |
| mineral | alloy | **RAW_ADAMANTINE** | crystalline cubes | light bluish grey | 170 |
| mineral | ??? | **SLADE** | fibrous or amorphous | dark grey | 142 |

### inorganic_stone_gem

To be fair, most all of these gems are minerals, often identical to some of the minerals in the previous section.

| Type | Subtype | Name | Habit | Colors | Tile |
| --- | --- | --- | --- | --- | --- |
| mineral | oxide | **ONYX** | parallel light bands against dark | black or red | 137 |
| mineral | oxide | **MORION**<sup>15</sup> | sharp facets, mostly opaque | black | 140 |
| mineral | silicate | **SHORL** | faceted or striated columns | black | 140 |
| mineral | silicate | **LACE AGATE** | heavily banded | light shades, often blue | 136 |
| mineral |  | **BLUE JADE** |  || 171 |
| mineral |  | **LAPIS LAZULI** |  || 171 |
| mineral |  | **PRASE** |  || 171 |
| mineral |  | **PRASE OPAL** |  || 171 |
| mineral |  | **BLOODSTONE** |  || 171 |
| mineral |  | **MOSS AGATE** | heavily banded | dark green | 136 |
| mineral |  | **MOSS OPAL** |  || 171 |
| mineral |  | **VARISCITE** |  || 171 |
| mineral |  | **CHRYSOPRASE** |  || 171 |
| mineral |  | **CHRYSOCOLLA** |  || 171 |
| mineral |  | **SARD** |  || 171 |
| mineral |  | **CARNELIAN** |  || 171 |
| mineral |  | **BANDED AGATE** | heavily banded | warm tones, whites, reds | 136 |
| mineral |  | **SARDONYX** |  || 171 |
| mineral |  | **CHERRY OPAL** |  || 171 |
| mineral |  | **LAVENDER JADE** |  || 171 |
| mineral |  | **PINK JADE** |  || 171 |
| mineral |  | **TUBE AGATE** | heavily circular banding | creams and reds | 136 |
| mineral |  | **FIRE AGATE** | rounded formations | irridescent | 139 |
| mineral |  | **PLUME AGATE** | heavily plumed banding | creams and reds | 136 |
| mineral |  | **BROWN JASPER** |  || 171 |
| mineral |  | **PICTURE JASPER** |  || 171 |
| mineral |  | **SMOKY QUARTZ** |  || 171 |
| mineral |  | **WAX OPAL** |  || 171 |
| mineral |  | **WOOD OPAL** |  || 171 |
| mineral |  | **AMBER OPAL** |  || 171 |
| mineral |  | **GOLD OPAL** |  || 171 |
| mineral |  | **CITRINE** |  || 171 |
| mineral |  | **YELLOW JASPER** |  || 171 |
| mineral |  | **TIGEREYE** |  || 171 |
| mineral |  | **TIGER IRON** |  || 171 |
| mineral |  | **SUNSTONE** |  || 171 |
| mineral |  | **RESIN OPAL** |  || 171 |
| mineral |  | **PYRITE** |  || 171 |
| mineral |  | **CLEAR TOURMALINE** |  || 171 |
| mineral |  | **GRAY CHALCEDONY** |  || 171 |
| mineral |  | **DENDRITIC AGATE** | heavily tree-like inclusions | black and white | 136 |
| mineral |  | **SHELL OPAL** |  || 171 |
| mineral |  | **BONE OPAL** |  || 171 |
| mineral |  | **WHITE CHALCEDONY** |  || 171 |
| mineral |  | **FORTIFICATION AGATE** | heavily banded | creams and reds | 136 |
| mineral |  | **MILK QUARTZ** |  || 171 |
| mineral |  | **MOONSTONE** |  || 171 |
| mineral |  | **WHITE JADE** |  || 171 |
| mineral |  | **JASPER OPAL** |  || 171 |
| mineral |  | **PINEAPPLE OPAL** |  || 171 |
| mineral |  | **ONYX OPAL** |  || 171 |
| mineral |  | **MILK OPAL** |  || 171 |
| mineral |  | **PIPE OPAL** |  || 171 |
| mineral |  | **AVENTURINE** |  || 171 |
| mineral |  | **TURQUOISE** |  || 171 |
| mineral |  | **QUARTZ_ROSE** |  || 171 |
| mineral |  | **CRYSTAL_ROCK** |  || 171 |
| mineral |  | **BLACK ZIRCON** |  || 171 |
| mineral |  | **BLACK PYROPE** |  || 171 |
| mineral |  | **MELANITE** |  || 171 |
| mineral |  | **INDIGO TOURMALINE** |  || 171 |
| mineral |  | **BLUE GARNET** |  || 171 |
| mineral |  | **TSAVORITE** |  || 171 |
| mineral |  | **GREEN TOURMALINE** |  || 171 |
| mineral |  | **DEMANTOID** |  || 171 |
| mineral |  | **GREEN ZIRCON** |  || 171 |
| mineral |  | **GREEN JADE** |  || 171 |
| mineral |  | **HELIODOR** |  || 171 |
| mineral |  | **PERIDOT** |  || 171 |
| mineral |  | **RED ZIRCON** |  || 171 |
| mineral |  | **RED TOURMALINE** |  || 171 |
| mineral |  | **RED PYROPE** |  || 171 |
| mineral |  | **ALMANDINE** |  || 171 |
| mineral |  | **RED GROSSULAR** |  || 171 |
| mineral |  | **PINK TOURMALINE** |  || 171 |
| mineral |  | **RED BERYL** |  || 171 |
| mineral |  | **FIRE OPAL** |  || 171 |
| mineral |  | **RHODOLITE** |  || 171 |
| mineral |  | **SPINEL_PURPLE** |  || 171 |
| mineral |  | **ALEXANDRITE** |  || 171 |
| mineral |  | **TANZANITE** |  || 171 |
| mineral |  | **MORGANITE** |  || 171 |
| mineral |  | **VIOLET SPESSARTINE** |  || 171 |
| mineral |  | **PINK GARNET** |  || 171 |
| mineral |  | **KUNZITE** |  || 171 |
| mineral |  | **CINNAMON GROSSULAR** |  || 171 |
| mineral |  | **HONEY YELLOW BERYL** |  || 171 |
| mineral |  | **JELLY OPAL** |  || 171 |
| mineral |  | **BROWN ZIRCON** |  || 171 |
| mineral |  | **YELLOW ZIRCON** |  || 171 |
| mineral |  | **GOLDEN BERYL** |  || 171 |
| mineral |  | **YELLOW SPESSARTINE** |  || 171 |
| mineral |  | **TOPAZ** |  || 171 |
| mineral |  | **TOPAZOLITE** |  || 171 |
| mineral |  | **YELLOW GROSSULAR** |  || 171 |
| mineral |  | **RUBICELLE** |  || 171 |
| mineral |  | **CLEAR GARNET** |  || 171 |
| mineral |  | **GOSHENITE** |  || 171 |
| mineral |  | **CAT'S EYE** |  || 171 |
| mineral |  | **CLEAR ZIRCON** |  || 171 |
| mineral |  | **AMETHYST** |  || 171 |
| mineral |  | **AQUAMARINE** |  || 171 |
| mineral |  | **SPINEL_RED** |  || 171 |
| mineral |  | **CHRYSOBERYL** |  || 171 |
| mineral |  | **OPAL_PFIRE** |  || 171 |
| mineral |  | **OPAL_REDFLASH** |  || 171 |
| mineral |  | **OPAL_BLACK** |  || 171 |
| mineral |  | **OPAL_WHITE** |  || 171 |
| mineral |  | **OPAL_CRYSTAL** |  || 171 |
| mineral |  | **OPAL_CLARO** |  || 171 |
| mineral |  | **OPAL_LEVIN** |  || 171 |
| mineral |  | **OPAL_HARLEQUIN** |  || 171 |
| mineral |  | **OPAL_PINFIRE]** |  || 171 |
| mineral |  | **OPAL_BANDFIRE** |  || 171 |
| mineral |  | **DIAMOND_LY** |  || 171 |
| mineral |  | **DIAMOND_FY** |  || 171 |
| mineral |  | **EMERALD** |  || 171 |
| mineral |  | **RUBY** |  || 171 |
| mineral |  | **SAPPHIRE** |  || 171 |
| mineral |  | **DIAMOND_CLEAR** |  || 171 |
| mineral |  | **DIAMOND_RED** |  || 171 |
| mineral |  | **DIAMOND_GREEN** |  || 171 |
| mineral |  | **DIAMOND_BLUE** |  || 171 |
| mineral |  | **DIAMOND_YELLOW** |  || 171 |
| mineral |  | **DIAMOND_BLACK** |  || 171 |
| mineral |  | **SAPPHIRE_STAR** |  || 171 |
| mineral |  | **RUBY_STAR** |  || 171 |

## Constructions (Walls, Floors)

## Furnitures (Tables, Chairs, Racks, Bridges, Etc)

## Flora

## Trinkets, Tools, and Doodads

## Notes

1. Rock salt is not actually a rock, but a singular mineral called Halite.
2. Dolomite is also not a rock, but a singular whitish crystal.  Dolo*STONE* is the rock being referred to hear which consists, in large part, of dolomite mixed with other minerals.
3. Granites come in many hues which often have names of their own.  Red Granite, Pink Granite, White Granite, Black Granite, etc.
4. Schist also tends to come in a variety of predictable hues, often grey, brown, blue, and green.
5. Marble tends to come in a very wide array of variety, and should be split out into a few notable options.
6. Garnierite is not actually a recognized mineral as there appear to be a wide variety of alternative chemical associations (or even mineral associations that would make it a rock, instead) that produce effects confused as being the same thing.
7. All of the coals are technically biogenic ROCK produced through metamorphic processes from fossilized material... but the raws often classify them as minerals instead.
8. Jet is merely considered a particularly quality and workable form of lignite, which means it is still a metamorphic rock or biogenic 'mineraloid' at best.
9. Literally, brimstone is just a name for sulfur.
10. Olivine is simply the massive/less translucent form of Peridot, and vice versa.
11. Hornblende is not officially a mineral at all, but a common name for a population of similar minerals.
12. Serpentine is not any one mineral, but a grouping of similar minerals with similar qualities.
13. Alabaster is a common name for any of three minerals derived from calcite or gypsum, but is not a mineral itself.
14. Selenite is just another name for gypsum, which is already included in the raws.  Satinspar is ALSO the same thing as both selenite and gypsum.  Only difference in each is shape.
15. Morion and Smokey Quartz are just slight different shades of the same thing