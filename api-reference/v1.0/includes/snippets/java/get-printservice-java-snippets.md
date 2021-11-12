---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c71f45f87db46528847adaaab7eab820100df71b83308c5cc45ca6816d085f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106702"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintService printService = graphClient.print().services("{printServiceId}")
    .buildRequest()
    .get();

```