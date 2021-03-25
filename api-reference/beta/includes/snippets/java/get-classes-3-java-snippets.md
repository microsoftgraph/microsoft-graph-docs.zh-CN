---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34608f36d5f39a9e214347df88d6bebeae5da78b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208739"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassCollectionWithReferencesPage classes = graphClient.education().me().classes()
    .buildRequest()
    .get();

```