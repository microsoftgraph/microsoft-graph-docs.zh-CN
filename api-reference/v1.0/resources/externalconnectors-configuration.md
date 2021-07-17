---
title: 配置资源类型
description: 指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加应用程序 ID。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: cd8f4ad66a80873d24f6ed14785e1f24d88077c4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467277"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="b73c8-103">配置资源类型</span><span class="sxs-lookup"><span data-stu-id="b73c8-103">configuration resource type</span></span>

<span data-ttu-id="b73c8-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="b73c8-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="b73c8-105">指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加[应用程序 ID。](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="b73c8-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b73c8-106">属性</span><span class="sxs-lookup"><span data-stu-id="b73c8-106">Properties</span></span>
|<span data-ttu-id="b73c8-107">属性</span><span class="sxs-lookup"><span data-stu-id="b73c8-107">Property</span></span>|<span data-ttu-id="b73c8-108">类型</span><span class="sxs-lookup"><span data-stu-id="b73c8-108">Type</span></span>|<span data-ttu-id="b73c8-109">说明</span><span class="sxs-lookup"><span data-stu-id="b73c8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b73c8-110">authorizedAppIds</span><span class="sxs-lookup"><span data-stu-id="b73c8-110">authorizedAppIds</span></span>|<span data-ttu-id="b73c8-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b73c8-111">String collection</span></span>|<span data-ttu-id="b73c8-112">允许管理 externalConnection 和为 externalConnection 中的内容编制索引的已注册 Azure Active Directory 应用程序的应用程序 ID 的集合。</span><span class="sxs-lookup"><span data-stu-id="b73c8-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b73c8-113">关系</span><span class="sxs-lookup"><span data-stu-id="b73c8-113">Relationships</span></span>
<span data-ttu-id="b73c8-114">无。</span><span class="sxs-lookup"><span data-stu-id="b73c8-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b73c8-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b73c8-115">JSON representation</span></span>
<span data-ttu-id="b73c8-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b73c8-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.configuration"
}
-->
``` json
{
  "authorizedAppIds": [
    "String"
  ]
}
```

