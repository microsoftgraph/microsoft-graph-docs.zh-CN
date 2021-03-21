---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0305bf2f5168b1aaf3a6736685e5d3ec08a46d8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967202"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroupCollectionPage sectionGroups = graphClient.me().onenote().notebooks("{id}").sectionGroups()
    .buildRequest()
    .get();

```