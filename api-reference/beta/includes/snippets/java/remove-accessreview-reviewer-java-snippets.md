---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e86ce797f3f147b0ee70607cad2bd9f359d865ea
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976181"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").reviewers("006111db-0810-4494-a6df-904d368bd81b")
    .buildRequest()
    .delete();

```