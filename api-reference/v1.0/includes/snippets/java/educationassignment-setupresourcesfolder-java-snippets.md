---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4138ea7447e874e4612f4a43aa4bdff786cc04b3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020067"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("955e0bd5-52c2-41ad-b7e8-5b33a18c5e78").assignments("18d17255-3278-49fb-8da7-d095b7f610c4")
    .setUpResourcesFolder()
    .buildRequest()
    .post();

```