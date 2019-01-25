---
title: fileHashType 枚举
description: 文件哈希类型的枚举。
localization_priority: Normal
ms.openlocfilehash: 082fdd9cdad6c3ec1ea4e07020983ac0bac7ed65
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518378"
---
# <a name="filehashtype-enum"></a>fileHashType 枚举

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

文件哈希类型的枚举。

## <a name="members"></a>成员

|成员|值|说明|
|:---|:---|:---|
|unknown|0%|未知的类型。|
|sha1|$1|SHA1 哈希值类型。|
|SHA256|-2| SHA256 哈希值类型。|
|MD5|-3| MD5 哈希值类型。|
|authenticodeHash256|-4| AuthenticodeHash256 哈希值类型。|
|lsHash|$-5| LsHash 哈希值类型。|
|ctph|-6| CTPH 哈希值类型。|
|peSha1|-7| PESHA1 哈希值类型。|
|peSha256|-8| PESHA256 哈希值类型。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/filehashtypeenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
