---
title: fileHash 资源类型
description: 包含有关文件哈希 (加密和位置敏感) 的状态信息。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: aabe56237ea44285c93f802268bd68688f16aa05
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030378"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="130a8-103">fileHash 资源类型</span><span class="sxs-lookup"><span data-stu-id="130a8-103">fileHash resource type</span></span>

<span data-ttu-id="130a8-104">包含有关文件哈希 (加密和位置敏感) 的状态信息。</span><span class="sxs-lookup"><span data-stu-id="130a8-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="130a8-105">属性</span><span class="sxs-lookup"><span data-stu-id="130a8-105">Properties</span></span>

| <span data-ttu-id="130a8-106">属性</span><span class="sxs-lookup"><span data-stu-id="130a8-106">Property</span></span>     | <span data-ttu-id="130a8-107">类型</span><span class="sxs-lookup"><span data-stu-id="130a8-107">Type</span></span>        | <span data-ttu-id="130a8-108">说明</span><span class="sxs-lookup"><span data-stu-id="130a8-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="130a8-109">hashType</span><span class="sxs-lookup"><span data-stu-id="130a8-109">hashType</span></span>|<span data-ttu-id="130a8-110">fileHashType</span><span class="sxs-lookup"><span data-stu-id="130a8-110">fileHashType</span></span>|<span data-ttu-id="130a8-111">文件哈希类型。</span><span class="sxs-lookup"><span data-stu-id="130a8-111">File hash type.</span></span> <span data-ttu-id="130a8-112">可取值为：`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256`。</span><span class="sxs-lookup"><span data-stu-id="130a8-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="130a8-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="130a8-113">hashValue</span></span>|<span data-ttu-id="130a8-114">String</span><span class="sxs-lookup"><span data-stu-id="130a8-114">String</span></span>|<span data-ttu-id="130a8-115">文件哈希值。</span><span class="sxs-lookup"><span data-stu-id="130a8-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="130a8-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="130a8-116">JSON representation</span></span>

<span data-ttu-id="130a8-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="130a8-117">The following is a JSON representation of the resource.</span></span>

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
