---
title: customSubjectAlternativeName 资源类型
description: 自定义主题备用名称定义
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2d621b67cffcf676dcd35889907eb5f9ca34504
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729796"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="3e804-103">customSubjectAlternativeName 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e804-103">customSubjectAlternativeName resource type</span></span>

<span data-ttu-id="3e804-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e804-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e804-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e804-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e804-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e804-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e804-107">自定义主题备用名称定义</span><span class="sxs-lookup"><span data-stu-id="3e804-107">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="3e804-108">属性</span><span class="sxs-lookup"><span data-stu-id="3e804-108">Properties</span></span>
|<span data-ttu-id="3e804-109">属性</span><span class="sxs-lookup"><span data-stu-id="3e804-109">Property</span></span>|<span data-ttu-id="3e804-110">类型</span><span class="sxs-lookup"><span data-stu-id="3e804-110">Type</span></span>|<span data-ttu-id="3e804-111">说明</span><span class="sxs-lookup"><span data-stu-id="3e804-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e804-112">sanType</span><span class="sxs-lookup"><span data-stu-id="3e804-112">sanType</span></span>|[<span data-ttu-id="3e804-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3e804-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3e804-114">自定义 SAN 类型。</span><span class="sxs-lookup"><span data-stu-id="3e804-114">Custom SAN Type.</span></span> <span data-ttu-id="3e804-115">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="3e804-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="3e804-116">name</span><span class="sxs-lookup"><span data-stu-id="3e804-116">name</span></span>|<span data-ttu-id="3e804-117">String</span><span class="sxs-lookup"><span data-stu-id="3e804-117">String</span></span>|<span data-ttu-id="3e804-118">自定义 SAN 名称</span><span class="sxs-lookup"><span data-stu-id="3e804-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e804-119">关系</span><span class="sxs-lookup"><span data-stu-id="3e804-119">Relationships</span></span>
<span data-ttu-id="3e804-120">无</span><span class="sxs-lookup"><span data-stu-id="3e804-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e804-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e804-121">JSON Representation</span></span>
<span data-ttu-id="3e804-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e804-122">Here is a JSON representation of the resource.</span></span>
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





