---
title: fileHash 资源类型
description: 包含有关文件哈希（加密和位置敏感）的状态信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a163a89e1e7ca7cb2a6bdf4c65945a601323d8fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498236"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="8f59a-103">fileHash 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f59a-103">fileHash resource type</span></span>

<span data-ttu-id="8f59a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8f59a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f59a-105">包含有关文件哈希（加密和位置敏感）的状态信息。</span><span class="sxs-lookup"><span data-stu-id="8f59a-105">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="8f59a-106">属性</span><span class="sxs-lookup"><span data-stu-id="8f59a-106">Properties</span></span>

| <span data-ttu-id="8f59a-107">属性</span><span class="sxs-lookup"><span data-stu-id="8f59a-107">Property</span></span>     | <span data-ttu-id="8f59a-108">类型</span><span class="sxs-lookup"><span data-stu-id="8f59a-108">Type</span></span>        | <span data-ttu-id="8f59a-109">说明</span><span class="sxs-lookup"><span data-stu-id="8f59a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f59a-110">hashType</span><span class="sxs-lookup"><span data-stu-id="8f59a-110">hashType</span></span>|<span data-ttu-id="8f59a-111">[fileHashType](filehashtypeenumtype.md)枚举</span><span class="sxs-lookup"><span data-stu-id="8f59a-111">[fileHashType](filehashtypeenumtype.md) enum</span></span>|<span data-ttu-id="8f59a-112">文件哈希类型。</span><span class="sxs-lookup"><span data-stu-id="8f59a-112">File hash type.</span></span> <span data-ttu-id="8f59a-113">可取值为：`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256`。</span><span class="sxs-lookup"><span data-stu-id="8f59a-113">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="8f59a-114">hashValue</span><span class="sxs-lookup"><span data-stu-id="8f59a-114">hashValue</span></span>|<span data-ttu-id="8f59a-115">String</span><span class="sxs-lookup"><span data-stu-id="8f59a-115">String</span></span>|<span data-ttu-id="8f59a-116">文件哈希值。</span><span class="sxs-lookup"><span data-stu-id="8f59a-116">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f59a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f59a-117">JSON representation</span></span>

<span data-ttu-id="8f59a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f59a-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
