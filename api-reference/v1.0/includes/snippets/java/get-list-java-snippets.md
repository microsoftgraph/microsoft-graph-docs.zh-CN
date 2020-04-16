---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99fdfcaef3034c21d847411d930cb0a91f2f3633
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2020
ms.locfileid: "43512267"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = graphClient.sites("{site-id}").lists("{list-title}")
    .buildRequest()
    .get();

```