---
title: groupPolicyObjectFile 资源类型
description: 由管理员上载的组策略对象文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b28ba6364f3261a7cd341870de402dc9332c87b4
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539195"
---
# <a name="grouppolicyobjectfile-resource-type"></a><span data-ttu-id="a5c81-103">groupPolicyObjectFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5c81-103">groupPolicyObjectFile resource type</span></span>

> <span data-ttu-id="a5c81-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a5c81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5c81-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5c81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5c81-106">由管理员上载的组策略对象文件。</span><span class="sxs-lookup"><span data-stu-id="a5c81-106">The Group Policy Object file uploaded by admin.</span></span>

## <a name="properties"></a><span data-ttu-id="a5c81-107">属性</span><span class="sxs-lookup"><span data-stu-id="a5c81-107">Properties</span></span>
|<span data-ttu-id="a5c81-108">属性</span><span class="sxs-lookup"><span data-stu-id="a5c81-108">Property</span></span>|<span data-ttu-id="a5c81-109">类型</span><span class="sxs-lookup"><span data-stu-id="a5c81-109">Type</span></span>|<span data-ttu-id="a5c81-110">说明</span><span class="sxs-lookup"><span data-stu-id="a5c81-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5c81-111">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="a5c81-111">ouDistinguishedName</span></span>|<span data-ttu-id="a5c81-112">字符串</span><span class="sxs-lookup"><span data-stu-id="a5c81-112">String</span></span>|<span data-ttu-id="a5c81-113">OU 的可分辨名称。</span><span class="sxs-lookup"><span data-stu-id="a5c81-113">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="a5c81-114">内容</span><span class="sxs-lookup"><span data-stu-id="a5c81-114">content</span></span>|<span data-ttu-id="a5c81-115">String</span><span class="sxs-lookup"><span data-stu-id="a5c81-115">String</span></span>|<span data-ttu-id="a5c81-116">组策略对象文件内容。</span><span class="sxs-lookup"><span data-stu-id="a5c81-116">The Group Policy Object file content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5c81-117">关系</span><span class="sxs-lookup"><span data-stu-id="a5c81-117">Relationships</span></span>
<span data-ttu-id="a5c81-118">无</span><span class="sxs-lookup"><span data-stu-id="a5c81-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5c81-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5c81-119">JSON Representation</span></span>
<span data-ttu-id="a5c81-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5c81-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPolicyObjectFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "ouDistinguishedName": "String",
  "content": "String"
}
```



