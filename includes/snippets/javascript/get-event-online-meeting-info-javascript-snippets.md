---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c01a34940f0ef6f6a6d27d527353cd7196db312204ae7cd79c1f11624ffdcd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkADAGu0AABIGYDZAAA=')
    .select('isOnlineMeeting,onlineMeetingProvider,onlineMeeting')
    .get();

```