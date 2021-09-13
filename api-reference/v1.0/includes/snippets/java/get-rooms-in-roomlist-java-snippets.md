---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4ae70ff265f126c5fafb4f8f5bab780fd7319396b738c488899a2f32ead7eea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219327"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RoomCollectionPage rooms = graphClient.places("bldg2@contoso.com").microsoft.graph.roomlist().rooms()
    .buildRequest()
    .get();

```