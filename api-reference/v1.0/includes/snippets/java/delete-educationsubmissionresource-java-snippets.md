---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14266a5e0650ba67f7e9970f52978439b4d439c73d09f6730f7e4308a8c28966
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277676"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8").submissions("fbe51c90-78b7-418a-b5f3-871bf8d8d21e").resources("f2387c3b-ec39-4bf2-a399-d7242677f024")
    .buildRequest()
    .delete();

```