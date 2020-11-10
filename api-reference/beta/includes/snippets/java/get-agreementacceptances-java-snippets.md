---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ad47a0dde024f27eeb1c17a68d45f5041512076
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973809"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAgreementAcceptanceCollectionWithReferencesPage agreementAcceptances = graphClient.me().agreementAcceptances()
    .buildRequest()
    .get();

```