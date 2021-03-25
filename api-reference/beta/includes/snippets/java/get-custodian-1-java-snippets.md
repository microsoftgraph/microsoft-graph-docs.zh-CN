---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c7349efe5ddd2da8f9a8ba8c58c95a009b0dad1
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209590"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CustodianCollectionPage custodians = graphClient.compliance().ediscovery().cases("2192ca408ea2410eba3bec8ae873be6b").custodians()
    .buildRequest()
    .get();

```