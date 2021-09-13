---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfc3acf51236a2eefd3745e27d17d15c01c3883048260dc54089f68fb4cce8c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106472"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const apply = {
  criteria: {
    criterion1: 'criterion1-value',
    criterion2: 'criterion2-value',
    color: 'color-value',
    operator: {
    },
    icon: {
      set: 'set-value',
      index: 99
    },
    dynamicCriteria: 'dynamicCriteria-value',
    values: {
    },
    filterOn: 'filterOn-value'
  }
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply')
    .post(apply);

```