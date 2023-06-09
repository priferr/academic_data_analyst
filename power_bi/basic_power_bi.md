# Projects from Introduction to Power BI course at Datacamp

This document contains an overview of the habilities used and developed to work with Power BI.

The Datacamp course emphasizes that it is just the surface of the power of this tool, but that it allows deepening the practice on real jobs. 

## Basic of Power BI



> **Note:** your visual class name must match what is defined in your `pbiviz.json` file.

```typescript
class MyVisual implements IVisual {
    
    constructor(options: VisualConstructorOptions) {
        //one time setup code goes here (called once)
    }
    
    public update(options: VisualUpdateOptions): void {
        //code to update your visual goes here (called on all view or data changes)
    }

    public enumerateObjectInstances(options: EnumerateVisualObjectInstancesOptions): VisualObjectInstanceEnumeration {
        //returns objects to populate the property pane (called for each object defined in capabilities)
    }
    
    public destroy(): void {
        //one time cleanup code goes here (called once)
    }
}
```

[Learn more about IVisual Api](IVisualApi.md)

## Visual Selection

Visuals can allow the user to select data points or categories by clicking them with the mouse.
Visual selection can be used to filter and behave with other visuals.

![](../images/MultiVisualSelection.png)

[Learn more about Visual Selection](Selection.md)
