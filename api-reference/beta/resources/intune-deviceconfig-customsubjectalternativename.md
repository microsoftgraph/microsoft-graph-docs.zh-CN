---
title: customSubjectAlternativeName 资源类型
description: 自定义的 Subject Alternative Name 定义
author: tfitzmac
ms.openlocfilehash: 5ed3f62cef38340ae7204b98e1fc984ba9bcb9cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349313"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="453d8-103">customSubjectAlternativeName 资源类型</span><span class="sxs-lookup"><span data-stu-id="453d8-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="453d8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="453d8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="453d8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="453d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="453d8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="453d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="453d8-107">自定义的 Subject Alternative Name 定义</span><span class="sxs-lookup"><span data-stu-id="453d8-107">Custom Subject Alternative Name definition</span></span>
## <a name="properties"></a><span data-ttu-id="453d8-108">属性</span><span class="sxs-lookup"><span data-stu-id="453d8-108">Properties</span></span>
|<span data-ttu-id="453d8-109">属性</span><span class="sxs-lookup"><span data-stu-id="453d8-109">Property</span></span>|<span data-ttu-id="453d8-110">类型</span><span class="sxs-lookup"><span data-stu-id="453d8-110">Type</span></span>|<span data-ttu-id="453d8-111">说明</span><span class="sxs-lookup"><span data-stu-id="453d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="453d8-112">sanType</span><span class="sxs-lookup"><span data-stu-id="453d8-112">sanType</span></span>|[<span data-ttu-id="453d8-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="453d8-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="453d8-114">自定义 SAN 类型。</span><span class="sxs-lookup"><span data-stu-id="453d8-114">Custom SAN Type.</span></span> <span data-ttu-id="453d8-115">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="453d8-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="453d8-116">name</span><span class="sxs-lookup"><span data-stu-id="453d8-116">name</span></span>|<span data-ttu-id="453d8-117">字符串</span><span class="sxs-lookup"><span data-stu-id="453d8-117">String</span></span>|<span data-ttu-id="453d8-118">自定义 SAN 名称</span><span class="sxs-lookup"><span data-stu-id="453d8-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="453d8-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="453d8-119">Relationships</span></span>
<span data-ttu-id="453d8-120">无</span><span class="sxs-lookup"><span data-stu-id="453d8-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="453d8-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="453d8-121">JSON Representation</span></span>
<span data-ttu-id="453d8-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="453d8-122">Here is a JSON representation of the resource.</span></span>
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





