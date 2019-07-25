---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 32681c93eceba7c7782702a321b3b8dc353ba447
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877212"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ILocaleInfoCollectionPage supportedLanguages = graphClient.me().outlook()
    .supportedLanguages()
    .buildRequest()
    .get();

```