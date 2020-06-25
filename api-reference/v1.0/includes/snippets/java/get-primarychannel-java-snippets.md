---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23ef32ae0d759091b5962c357a63a75ba91c9801
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863892"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = graphClient.teams("{id}").primaryChannel()
    .buildRequest()
    .get();

```