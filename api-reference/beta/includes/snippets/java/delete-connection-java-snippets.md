---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ffb4af9779ba248511d5d5828abd97e4acf0c3d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968918"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.connections("contosohr")
    .buildRequest()
    .delete();

```