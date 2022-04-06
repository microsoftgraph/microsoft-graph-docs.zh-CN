---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d768fcca62d1518c0776c3c277fd4a7f52cd804
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759262"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.applications("fd918e4b-c821-4efb-b50a-5eddd23afc6f").extensionProperties("1f0f15e3-925d-40f0-8fc8-9d3ad135bce0")
    .buildRequest()
    .delete();

```