---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 771bf12285b869d5ff5e79dbf3f7537e45e6cf62
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37999471"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String keyId = "f0b0b335-1d71-4883-8f98-567911bfdca6";

graphClient.applications("{id}")
    .removePassword(keyId)
    .buildRequest()
    .post();

```