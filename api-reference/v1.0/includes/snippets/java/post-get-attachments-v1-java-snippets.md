---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c2ddcc3a9b16cd429053330f53ac965ca5a24868
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636794"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAttachmentCollectionPage attachments = graphClient.groups("1848753d-185d-4c08-a4e4-6ee40521d115").threads("AAQkADJfolA==").posts("AAMkADJ-aHAAA=").attachments()
    .buildRequest()
    .get();

```