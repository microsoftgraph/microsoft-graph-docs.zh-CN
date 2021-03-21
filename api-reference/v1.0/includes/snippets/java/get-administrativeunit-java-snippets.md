---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcabd0b3b2968c0d5aed7b4f6daf1d927f0a2c5e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969826"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = graphClient.directory().administrativeUnits("{id}")
    .buildRequest()
    .get();

```