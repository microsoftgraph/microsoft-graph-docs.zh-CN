---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 303cc037ed77c8d3506005e2336d67932f34dbee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974547"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationalActivityCollectionPage educationalActivities = graphClient.me().profile().educationalActivities()
    .buildRequest()
    .get();

```