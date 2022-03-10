---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 537b33749afc176364dc17eff6f781e5a1ede10f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
    templateId: '62375ab9-6b52-47ed-826b-58e47e0e304b',
    values: [
        {
            name: 'GuestUsageGuidelinesUrl',
            value: 'https://privacy.contoso.com/privacystatement'
        },
        {
            name: 'EnableMSStandardBlockedWords',
            value: 'true'
        },
        {
            name: 'EnableMIPLabels',
            value: 'true'
        },
        {
            name: 'PrefixSuffixNamingRequirement',
            value: '[Contoso-][GroupName]'
        }
    ]
};

await client.api('/groupSettings')
    .post(groupSetting);

```