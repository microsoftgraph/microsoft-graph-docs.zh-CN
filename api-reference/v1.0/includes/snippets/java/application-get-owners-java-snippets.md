---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67a21f9447e399c0b2ba902ad59ea94844de239d
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999113"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage owners = graphClient.applications("{id}").owners()
    .buildRequest()
    .get();

```