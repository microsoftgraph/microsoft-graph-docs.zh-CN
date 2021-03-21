---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af26f5372ebcc777c4e29632ae8d582eff884d72
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983960"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{printerShareId}").allowedUsers("{userId}").reference()
    .buildRequest()
    .delete();

```