---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 858472dc8dbc94ce13f09c004256ee69f2868157b4d778cf15c07b78fba2e6fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162573"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const listItem = {
  fields: {
    Title: 'Widget',
    Color: 'Purple',
    Weight: 32
  }
};

await client.api('/sites/{site-id}/lists/{list-id}/items')
    .post(listItem);

```