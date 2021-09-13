---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5ba417b7ec2b0c69e972b62a43eb1e530131bcb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022492"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.external().connections("contosohr").groups("31bea3d537902000")
    .buildRequest()
    .delete();

```