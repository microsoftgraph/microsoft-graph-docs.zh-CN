---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 140174b88fbcd648383ad3b82079c3e711ddab4980d15b698b06a1458ee908eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274009"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = graphClient.education().schools("2961761D-8094-4183-A9F6-8E36E966C7D9").administrativeUnit()
    .buildRequest()
    .get();

```