---
title: customSubjectAlternativeName 资源类型
description: 自定义的 Subject Alternative Name 定义
ms.openlocfilehash: 14d6c24cd5e8c087b81fa51194301da522d169b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045301"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="64a2c-103">customSubjectAlternativeName 资源类型</span><span class="sxs-lookup"><span data-stu-id="64a2c-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="64a2c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="64a2c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64a2c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="64a2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64a2c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="64a2c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64a2c-107">自定义的 Subject Alternative Name 定义</span><span class="sxs-lookup"><span data-stu-id="64a2c-107">Custom Subject Alternative Name definition</span></span>
## <a name="properties"></a><span data-ttu-id="64a2c-108">属性</span><span class="sxs-lookup"><span data-stu-id="64a2c-108">Properties</span></span>
|<span data-ttu-id="64a2c-109">属性</span><span class="sxs-lookup"><span data-stu-id="64a2c-109">Property</span></span>|<span data-ttu-id="64a2c-110">类型</span><span class="sxs-lookup"><span data-stu-id="64a2c-110">Type</span></span>|<span data-ttu-id="64a2c-111">说明</span><span class="sxs-lookup"><span data-stu-id="64a2c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64a2c-112">sanType</span><span class="sxs-lookup"><span data-stu-id="64a2c-112">sanType</span></span>|[<span data-ttu-id="64a2c-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="64a2c-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="64a2c-114">自定义 SAN 类型。</span><span class="sxs-lookup"><span data-stu-id="64a2c-114">Custom SAN Type.</span></span> <span data-ttu-id="64a2c-115">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="64a2c-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="64a2c-116">name</span><span class="sxs-lookup"><span data-stu-id="64a2c-116">name</span></span>|<span data-ttu-id="64a2c-117">字符串</span><span class="sxs-lookup"><span data-stu-id="64a2c-117">String</span></span>|<span data-ttu-id="64a2c-118">自定义 SAN 名称</span><span class="sxs-lookup"><span data-stu-id="64a2c-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="64a2c-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="64a2c-119">Relationships</span></span>
<span data-ttu-id="64a2c-120">无</span><span class="sxs-lookup"><span data-stu-id="64a2c-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="64a2c-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64a2c-121">JSON Representation</span></span>
<span data-ttu-id="64a2c-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64a2c-122">Here is a JSON representation of the resource.</span></span>
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





