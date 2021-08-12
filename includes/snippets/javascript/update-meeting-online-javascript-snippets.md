---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8be1a67d2c59f47ae90b5e1123bc11b0b401dbe015c8fdf2c451a84950fbe16a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  isOnlineMeeting: true,
  onlineMeetingProvider: "teamsForBusiness"
};

let res = await client.api('/me/events/AAMkADAGu0AABIGYDaAAA=')
    .update(event);

```