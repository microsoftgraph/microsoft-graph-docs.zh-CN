---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 992d453263caef61e19a6205d224acf9c61ca683
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774571"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage members = graphClient.directoryRoles("{id}").members()
    .buildRequest()
    .get();

```