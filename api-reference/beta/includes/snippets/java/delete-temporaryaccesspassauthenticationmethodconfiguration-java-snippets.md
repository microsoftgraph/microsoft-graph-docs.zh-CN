---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb5a41dce65e4b97ecefa61dbd982dea5507bfbf
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443108"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("temporaryAccessPass`")
    .buildRequest()
    .delete();

```