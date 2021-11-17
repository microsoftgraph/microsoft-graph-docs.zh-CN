---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bbc354463ed9370a1054c33a2611c5c40b4380a7a692c1cb046dc0bf2464428
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163668"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().outlook().masterCategories("4b1c2495-54c9-4a5e-90a2-0ab0b31987d8")
    .buildRequest()
    .delete();

```