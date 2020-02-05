---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3887be27e41a33f873fa90dfc622518310f9f27c
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774501"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserCollectionPage members = graphClient.education().classes("{class-id}").members()
    .buildRequest()
    .get();

```