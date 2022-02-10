---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdc58ef2c6a7e8c8c88b0af1463843209138513e
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519336"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const customSecurityAttributeDefinition = {
    attributeSet: 'Engineering',
    description: 'Active projects for user',
    isCollection: true,
    isSearchable: true,
    name: 'Project',
    status: 'Available',
    type: 'String',
    usePreDefinedValuesOnly: true,
    allowedValues: [
        {
            id: 'Alpine',
            isActive: true
        },
        {
            id: 'Baker',
            isActive: true
        },
        {
            id: 'Cascade',
            isActive: true
        }
    ]
};

await client.api('/directory/customSecurityAttributeDefinitions')
    .version('beta')
    .post(customSecurityAttributeDefinition);

```