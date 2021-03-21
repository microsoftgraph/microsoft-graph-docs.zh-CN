---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3b8a88bba31b518fddca2be6bd6c46f81e2f9fd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984089"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationCollectionPage applications = graphClient.applications()
    .buildRequest()
    .get();

```