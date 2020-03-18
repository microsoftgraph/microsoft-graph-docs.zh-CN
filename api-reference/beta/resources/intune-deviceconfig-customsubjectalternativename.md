---
title: customSubjectAlternativeName 资源类型
description: 自定义主题备用名称定义
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 22f28942f891bc8ac72f6640091e0b8e1195f51f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795650"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="98a79-103">customSubjectAlternativeName 资源类型</span><span class="sxs-lookup"><span data-stu-id="98a79-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="98a79-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="98a79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98a79-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="98a79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98a79-106">自定义主题备用名称定义</span><span class="sxs-lookup"><span data-stu-id="98a79-106">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="98a79-107">属性</span><span class="sxs-lookup"><span data-stu-id="98a79-107">Properties</span></span>
|<span data-ttu-id="98a79-108">属性</span><span class="sxs-lookup"><span data-stu-id="98a79-108">Property</span></span>|<span data-ttu-id="98a79-109">类型</span><span class="sxs-lookup"><span data-stu-id="98a79-109">Type</span></span>|<span data-ttu-id="98a79-110">说明</span><span class="sxs-lookup"><span data-stu-id="98a79-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98a79-111">sanType</span><span class="sxs-lookup"><span data-stu-id="98a79-111">sanType</span></span>|[<span data-ttu-id="98a79-112">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="98a79-112">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="98a79-113">自定义 SAN 类型。</span><span class="sxs-lookup"><span data-stu-id="98a79-113">Custom SAN Type.</span></span> <span data-ttu-id="98a79-114">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="98a79-114">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="98a79-115">name</span><span class="sxs-lookup"><span data-stu-id="98a79-115">name</span></span>|<span data-ttu-id="98a79-116">String</span><span class="sxs-lookup"><span data-stu-id="98a79-116">String</span></span>|<span data-ttu-id="98a79-117">自定义 SAN 名称</span><span class="sxs-lookup"><span data-stu-id="98a79-117">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="98a79-118">关系</span><span class="sxs-lookup"><span data-stu-id="98a79-118">Relationships</span></span>
<span data-ttu-id="98a79-119">无</span><span class="sxs-lookup"><span data-stu-id="98a79-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98a79-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98a79-120">JSON Representation</span></span>
<span data-ttu-id="98a79-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98a79-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```



