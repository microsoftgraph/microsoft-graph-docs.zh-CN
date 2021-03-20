---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47b2d60bc0ed0e18cdbbbf8c0d1a281c4f3834b9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976165"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationOutcomeCollectionPage outcomes = graphClient.education().me().assignments("{id}").submissions("{id}").outcomes()
    .buildRequest()
    .get();

```