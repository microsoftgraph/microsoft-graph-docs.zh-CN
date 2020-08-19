---
title: fileHash 资源类型
description: 包含有关文件哈希 (加密和位置敏感) 的状态信息。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d034d586bad1da54e57490e300b34191034a1657
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807827"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="922b1-103">fileHash 资源类型</span><span class="sxs-lookup"><span data-stu-id="922b1-103">fileHash resource type</span></span>

<span data-ttu-id="922b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="922b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="922b1-105">包含有关文件哈希 (加密和位置敏感) 的状态信息。</span><span class="sxs-lookup"><span data-stu-id="922b1-105">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="922b1-106">属性</span><span class="sxs-lookup"><span data-stu-id="922b1-106">Properties</span></span>

| <span data-ttu-id="922b1-107">属性</span><span class="sxs-lookup"><span data-stu-id="922b1-107">Property</span></span>     | <span data-ttu-id="922b1-108">类型</span><span class="sxs-lookup"><span data-stu-id="922b1-108">Type</span></span>        | <span data-ttu-id="922b1-109">说明</span><span class="sxs-lookup"><span data-stu-id="922b1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="922b1-110">hashType</span><span class="sxs-lookup"><span data-stu-id="922b1-110">hashType</span></span>|<span data-ttu-id="922b1-111">fileHashType</span><span class="sxs-lookup"><span data-stu-id="922b1-111">fileHashType</span></span>|<span data-ttu-id="922b1-112">文件哈希类型。</span><span class="sxs-lookup"><span data-stu-id="922b1-112">File hash type.</span></span> <span data-ttu-id="922b1-113">可取值为：`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256`。</span><span class="sxs-lookup"><span data-stu-id="922b1-113">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="922b1-114">hashValue</span><span class="sxs-lookup"><span data-stu-id="922b1-114">hashValue</span></span>|<span data-ttu-id="922b1-115">String</span><span class="sxs-lookup"><span data-stu-id="922b1-115">String</span></span>|<span data-ttu-id="922b1-116">文件哈希值。</span><span class="sxs-lookup"><span data-stu-id="922b1-116">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="922b1-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="922b1-117">JSON representation</span></span>

<span data-ttu-id="922b1-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="922b1-118">The following is a JSON representation of the resource.</span></span>

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
