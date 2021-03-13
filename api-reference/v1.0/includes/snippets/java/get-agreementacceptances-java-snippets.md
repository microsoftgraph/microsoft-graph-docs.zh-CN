---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ad47a0dde024f27eeb1c17a68d45f5041512076
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777459"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAgreementAcceptanceCollectionWithReferencesPage agreementAcceptances = graphClient.me().agreementAcceptances()
    .buildRequest()
    .get();

```