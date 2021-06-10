---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c3e9b9f6925da01d60df4ccf798540ff2c013f0
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870456"
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