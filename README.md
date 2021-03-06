# Automatic human timestamp properties in Laravel

This package provides a trait you can add to an Eloquent model that will automatically create human-readable timestamp diffs using Carbon.

## Installation

To install the package run:

```
composer require chrisdicarlo/eloquent-human-timestamps
```

## Setup

Add the ChrisDiCarlo\EloquentHumanTimestamps\HumanTimestamps trait to a model that has timestamp columns, e.g.:

```

use ChrisDiCarlo\EloquentHumanTimestamps\HumanTimestamps;

class Foobar
{
  
    use HumanTimestamps;

   ...

}
```

## Usage

To get the human-readable attribute, simply retrieve the timestamp normally but append **_for_humans** to the name, e.g. created_at_for_humans, updated_at_for_humans.

