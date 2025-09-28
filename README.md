# ⚠️⚠️⚠️ DEPRECATED: Use the UniSports Catalog instead:  https://github.com/OatsCG/UniSports-Catalog/tree/main/UTM

# UTM-Drop-Ins-Schedule
#### A downloadable schedule of University of Toronto Mississauga Drop-In Sports.

version.txt stores the version and date of when events.json was last updated.

## [App Data Pipeline](UTMSportsDataPipeline.pdf)

## Schema
```ts
{
    "categories": [
        {
            "title": String,
            "symbol": String,
            "isChip": Bool,
            "isMedal": Bool
        },
        ...
    ],
    "events": [
        {
            "id": Int,
            "url": String, // URL
            "title": String,
            "description": String,
            "image": String, // URL
            "start_date": String, // Date String %Y-%m-%d %H:%M:%S
            "end_date": String, // Date String %Y-%m-%d %H:%M:%S
            "venue": String,
            "ticket_label": String,
            "ticket_url": String, // URL
            "sortCategory": String,
            "symbol": String,
            "womens": Bool,
            "weeklyRepetitions": [String] // su, mo, tu, we, th, fr, sa
        },
        ...
    ],
    "featured": [
        {
            "id": Int,
            "url": String, // URL
            "title": String,
            "description": String,
            "image": String, // URL
            "start_date": String, // Date String %Y-%m-%d %H:%M:%S
            "end_date": String, // Date String %Y-%m-%d %H:%M:%S
            "venue": String,
            "ticket_label": String,
            "ticket_url": String, // URL
            "sortCategory": String,
            "symbol": String,
            "womens": Bool,
            "weeklyRepetitions": [String] // su, mo, tu, we, th, fr, sa
        },
        ...
    ],
    "announcements": [
        {
            "id": Int,
            "title": String,
            "body": String,
            "type": Int // 0=>normal, 1=>closure, 2=>update, other=>gray
        },
        ...
    ]
}
```


## To Note
- "featured" events exist in "events" as well
