# Бекап сервера

### Как использовать?
Чтобы сохранить бекап сервера пропишите команду /backup_save , а чтобы загрузить - /backup_load

### Файл бекапа
Именно этот файл используется для загрузки бекапа. Устройство файла с бекапом:
```python
"""
# {guild_id}.json
{
    'channels': [
        [  # text
            {
             'category_id': Optional[int],
             'name': str,
             'nsfw': bool,
             'position': int,
             'slowmode_delay': int,
             'topic': Optional[str],
             'default_auto_archive_duration': int,
             'default_thread_slowmode_delay': int,
             'id': int
            },
        ],

        [  # voice
            {
             'bitrate': int,
             'category_id': Optional[int],
             'name': str,
             'nsfw': bool,
             'position': int,
             'rtc_region': Optional[str],
             'slowmode_delay': int,
             'user_limit': int,
             'video_quality_mode': List[str, int],
             'id': int
            },
        ],

        [  # category
            {
             'id': int,
             'name': str,
             'nsfw': bool,
             'position': int
            },
        ],

        [  # forums
            {
             'category_id': Optional[int],
             'name': str,
             'nsfw': bool,
             'default_layout': int,
             'default_reaction_emoji': Optional[str],
             'default_sort_order': Optional[int],
             'position': int,
             'slowmode_delay': int,
             'topic': Optional[str],
             'default_auto_archive_duration': int,
             'default_thread_slowmode_delay': int,
             'id': int
            },
        ],

        [  # stages
            {
             'bitrate': int,
             'category_id': Optional[int],
             'name': str,
             'nsfw': bool,
             'position': int,
             'rtc_region': Optional[str],
             'slowmode_delay': int,
             'user_limit': int,
             'video_quality_mode': List[str, int],
             'id': int
            },
        ]
    ],

    'roles': [
        {
         'color_value': int,
         'hoist': bool,
         'mentionable': bool,
         'name': str,
         'permission_value': int,
         'position': int,
         'id': int
        },
    ],

    'date': str
}
"""
```
