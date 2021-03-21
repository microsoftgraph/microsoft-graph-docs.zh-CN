---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e03e73572c4073ef245abe24bf1762f1b780e00d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981684"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRoot educationRoot = graphClient.education()
    .buildRequest()
    .get();

```