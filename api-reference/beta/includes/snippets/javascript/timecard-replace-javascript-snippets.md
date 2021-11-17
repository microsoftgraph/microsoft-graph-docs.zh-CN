---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 028b8ca5682570d178684fcbdf68593189695d2a57b1c18c38d8445d56f418ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103810"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeCard = {
    userId: '70e47528-2fae-42b5-9d8e-ee73ccd90603',
    state: 'clockedOut',
    confirmedBy: 'None',
    notes: null,
    clockInEvent: {
        dateTime: '2021-05-21T21:58:41.327Z',
        atApprovedLocation: null,
        notes: {
            contentType: 'text',
            content: 'update sample notes'
        }
    },
    clockOutEvent: {
        dateTime: '2021-05-21T22:01:46.205Z',
        atApprovedLocation: null,
        notes: {
            contentType: 'text',
            content: 'update sample notes'
        }
    },
    breaks: [
        {
            breakId: 'BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f',
            notes: null,
            start: {
                dateTime: '2021-05-21T21:59:59.328Z',
                atApprovedLocation: null,
                notes: {
                    contentType: 'text',
                    content: 'update sample notes'
                }
            },
            end: {
                dateTime: '2021-05-21T22:01:10.205Z',
                atApprovedLocation: null,
                notes: {
                    contentType: 'text',
                    content: 'update sample notes'
                }
            }
        }
    ]
};

await client.api('/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_3cd7413f-0337-433b-9a49-da0923185b3f')
    .version('beta')
    .put(timeCard);

```