---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dc2d9b7eabdfe8d05227105318d0a847cf325b0389eb88c3f0a55175625e872
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103857"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnectorCollectionWithReferencesPage connectors = graphClient.print().printers("{id}").connectors()
    .buildRequest()
    .get();

```