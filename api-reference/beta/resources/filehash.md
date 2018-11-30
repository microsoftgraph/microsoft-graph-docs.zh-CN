---
title: fileHash 资源类型
description: 包含有关文件哈希 （加密和位置） 的状态信息。
ms.openlocfilehash: 8f283046efc9b4af181cb33fb4e9ca63e4892b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045728"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="df455-103">fileHash 资源类型</span><span class="sxs-lookup"><span data-stu-id="df455-103">fileHash resource type</span></span>

<span data-ttu-id="df455-104">包含有关文件哈希 （加密和位置） 的状态信息。</span><span class="sxs-lookup"><span data-stu-id="df455-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="df455-105">属性</span><span class="sxs-lookup"><span data-stu-id="df455-105">Properties</span></span>

| <span data-ttu-id="df455-106">属性</span><span class="sxs-lookup"><span data-stu-id="df455-106">Property</span></span>     | <span data-ttu-id="df455-107">类型</span><span class="sxs-lookup"><span data-stu-id="df455-107">Type</span></span>        | <span data-ttu-id="df455-108">说明</span><span class="sxs-lookup"><span data-stu-id="df455-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df455-109">hashType</span><span class="sxs-lookup"><span data-stu-id="df455-109">hashType</span></span>|<span data-ttu-id="df455-110">[fileHashType](filehashtypeenumtype.md)枚举</span><span class="sxs-lookup"><span data-stu-id="df455-110">[fileHashType](filehashtypeenumtype.md) enum</span></span>|<span data-ttu-id="df455-111">文件哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="df455-111">File hash type.</span></span> <span data-ttu-id="df455-112">可取值为：`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256`。</span><span class="sxs-lookup"><span data-stu-id="df455-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="df455-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="df455-113">hashValue</span></span>|<span data-ttu-id="df455-114">字符串</span><span class="sxs-lookup"><span data-stu-id="df455-114">String</span></span>|<span data-ttu-id="df455-115">文件哈希值。</span><span class="sxs-lookup"><span data-stu-id="df455-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df455-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df455-116">JSON representation</span></span>

<span data-ttu-id="df455-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df455-117">The following is a JSON representation of the resource.</span></span>

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