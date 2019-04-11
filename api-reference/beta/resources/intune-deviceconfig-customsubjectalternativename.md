---
title: customSubjectAlternativeName 资源类型
description: 自定义主题备用名称定义
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03507d4e912af011db011283a95887590ab79801
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783949"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="de2f1-103">customSubjectAlternativeName 资源类型</span><span class="sxs-lookup"><span data-stu-id="de2f1-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="de2f1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="de2f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de2f1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de2f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de2f1-106">自定义主题备用名称定义</span><span class="sxs-lookup"><span data-stu-id="de2f1-106">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="de2f1-107">属性</span><span class="sxs-lookup"><span data-stu-id="de2f1-107">Properties</span></span>
|<span data-ttu-id="de2f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="de2f1-108">Property</span></span>|<span data-ttu-id="de2f1-109">类型</span><span class="sxs-lookup"><span data-stu-id="de2f1-109">Type</span></span>|<span data-ttu-id="de2f1-110">说明</span><span class="sxs-lookup"><span data-stu-id="de2f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de2f1-111">sanType</span><span class="sxs-lookup"><span data-stu-id="de2f1-111">sanType</span></span>|[<span data-ttu-id="de2f1-112">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="de2f1-112">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="de2f1-113">自定义 SAN 类型。</span><span class="sxs-lookup"><span data-stu-id="de2f1-113">Custom SAN Type.</span></span> <span data-ttu-id="de2f1-114">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute` 或 `domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="de2f1-114">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="de2f1-115">name</span><span class="sxs-lookup"><span data-stu-id="de2f1-115">name</span></span>|<span data-ttu-id="de2f1-116">String</span><span class="sxs-lookup"><span data-stu-id="de2f1-116">String</span></span>|<span data-ttu-id="de2f1-117">自定义 SAN 名称</span><span class="sxs-lookup"><span data-stu-id="de2f1-117">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="de2f1-118">关系</span><span class="sxs-lookup"><span data-stu-id="de2f1-118">Relationships</span></span>
<span data-ttu-id="de2f1-119">无</span><span class="sxs-lookup"><span data-stu-id="de2f1-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de2f1-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de2f1-120">JSON Representation</span></span>
<span data-ttu-id="de2f1-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de2f1-121">Here is a JSON representation of the resource.</span></span>
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





