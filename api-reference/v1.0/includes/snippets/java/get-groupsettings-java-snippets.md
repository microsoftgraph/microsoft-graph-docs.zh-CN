---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f0348ebbf5fe6741522db44004abf1de4c39a61
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979893"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSettingCollectionPage groupSettings = graphClient.groupSettings()
    .buildRequest()
    .get();

```