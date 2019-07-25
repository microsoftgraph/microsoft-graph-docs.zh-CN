---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9cd99c300e7b8d27ccfdbb7c5424bd0f1dc28d9b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877785"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookCategory outlookCategory = graphClient.me().outlook().masterCategories("de912e4d-c790-4da9-949c-ccd933aaa0f7")
    .buildRequest()
    .get();

```