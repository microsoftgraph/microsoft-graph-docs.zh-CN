---
title: fileHash 资源类型
description: 包含有关文件哈希 (加密和位置敏感) 的状态信息。
localization_priority: Normal
ms.openlocfilehash: f5d865a7ded230ca611b8628c3648ec1e331c67d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547604"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="8d3a0-103">fileHash 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d3a0-103">fileHash resource type</span></span>

<span data-ttu-id="8d3a0-104">包含有关文件哈希 (加密和位置敏感) 的状态信息。</span><span class="sxs-lookup"><span data-stu-id="8d3a0-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="8d3a0-105">属性</span><span class="sxs-lookup"><span data-stu-id="8d3a0-105">Properties</span></span>

| <span data-ttu-id="8d3a0-106">属性</span><span class="sxs-lookup"><span data-stu-id="8d3a0-106">Property</span></span>     | <span data-ttu-id="8d3a0-107">类型</span><span class="sxs-lookup"><span data-stu-id="8d3a0-107">Type</span></span>        | <span data-ttu-id="8d3a0-108">说明</span><span class="sxs-lookup"><span data-stu-id="8d3a0-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d3a0-109">hashType</span><span class="sxs-lookup"><span data-stu-id="8d3a0-109">hashType</span></span>|<span data-ttu-id="8d3a0-110">[fileHashType](filehashtypeenumtype.md)枚举</span><span class="sxs-lookup"><span data-stu-id="8d3a0-110">[fileHashType](filehashtypeenumtype.md) enum</span></span>|<span data-ttu-id="8d3a0-111">文件哈希类型。</span><span class="sxs-lookup"><span data-stu-id="8d3a0-111">File hash type.</span></span> <span data-ttu-id="8d3a0-112">可取值为：`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256`。</span><span class="sxs-lookup"><span data-stu-id="8d3a0-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="8d3a0-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="8d3a0-113">hashValue</span></span>|<span data-ttu-id="8d3a0-114">String</span><span class="sxs-lookup"><span data-stu-id="8d3a0-114">String</span></span>|<span data-ttu-id="8d3a0-115">文件哈希值。</span><span class="sxs-lookup"><span data-stu-id="8d3a0-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d3a0-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d3a0-116">JSON representation</span></span>

<span data-ttu-id="8d3a0-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d3a0-117">The following is a JSON representation of the resource.</span></span>

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
