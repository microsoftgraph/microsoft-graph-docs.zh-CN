---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef2d1470f1616acd7f50baceb1d712ffce3caa4b1780b177bc033123da47427e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333968"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnection externalConnection = graphClient.connections("contosohr")
    .buildRequest()
    .get();

```