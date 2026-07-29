# PvZ Skin

Plants vs. Zombies 2 LibGDX Scene2D UI skin.

> **Note:** This skin requires [TenPatch](https://github.com/raeleus/TenPatch). Ensure it is included in your project dependencies.

## Installation (Gradle)

```groovy
repositories {
    maven { url 'https://jitpack.io' }
}

dependencies {
    implementation 'com.github.pizpizi:pvz-skin:v0.1.0'
    implementation 'com.github.raeleus.TenPatch:tenpatch:5.2.3'
}
```

## Usage

```java
import pvz.skin.PvzSkin;

// 1. Load the skin
Skin skin = PvzSkin.get();

// 2. Create UI widgets using skin styles
TextButton button = new TextButton("Play", skin, "green_small");
Label label = new Label("PvZ UI", skin, "big_outline");

// 3. Add widgets to your Scene2D Stage
Stage stage = new Stage();
stage.addActor(button);
```