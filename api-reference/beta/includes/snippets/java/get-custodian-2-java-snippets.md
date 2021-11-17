---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ab6cf4c16ab91e826289adbf089a8da59c04213e9c154339b7b7f3391fde525
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219059"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Custodian custodian = graphClient.compliance().ediscovery().cases("2192ca408ea2410eba3bec8ae873be6b").custodians("45454331323337443946343043464239")
    .buildRequest()
    .get();

```