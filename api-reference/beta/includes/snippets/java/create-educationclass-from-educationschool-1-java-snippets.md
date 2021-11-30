---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 993d8a5022ad181b16b691894165219a5f71687720346dd1f958b7afd685ab0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378308"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11003").members("14008")
    .buildRequest()
    .delete();

```