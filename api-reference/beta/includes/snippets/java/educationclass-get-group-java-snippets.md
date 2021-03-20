---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 694c1d2130c1a4aef7f359b1e70d5ec780135537
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978385"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.education().classes("2961761D-8094-4183-A9F6-8E36E966C7D9").group()
    .buildRequest()
    .get();

```