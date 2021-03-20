---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57da0cba02bd43776c3056d67a2450df9f6d5aee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973385"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().me().rubrics("{id}")
    .buildRequest()
    .delete();

```