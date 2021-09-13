---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ae2371a8ebaa3e22e60c423ed10a5003207299080d8dc5ae22961e293b7709e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274253"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8").submissions("fbe51c90-78b7-418a-b5f3-871bf8d8d21e")
    .unsubmit()
    .buildRequest()
    .post();

```