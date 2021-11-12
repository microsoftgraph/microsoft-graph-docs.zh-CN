---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52b3ea59ca4999437e9a40f6ae21daf663bdd22d8f9a19abb9fd238ee6c930e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277863"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskTriggerCollectionPage taskTriggers = graphClient.print().printers("{printerId}").taskTriggers()
    .buildRequest()
    .get();

```