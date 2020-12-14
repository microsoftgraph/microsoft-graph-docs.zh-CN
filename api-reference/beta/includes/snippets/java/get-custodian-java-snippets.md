---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cf4850a0028214cb3828f8ef901976df25e2312
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657154"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICustodianCollectionPage custodians = graphClient.compliance().ediscovery().cases("2192ca408ea2410eba3bec8ae873be6b").custodians()
    .buildRequest()
    .get();

```