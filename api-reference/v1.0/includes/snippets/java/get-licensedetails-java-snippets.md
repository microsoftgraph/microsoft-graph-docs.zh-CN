---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0a7005197bfd7b2c5dd0e351ee179942672d5857
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888861"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ILicenseDetailsCollectionPage licenseDetails = graphClient.me().licenseDetails()
    .buildRequest()
    .get();

```