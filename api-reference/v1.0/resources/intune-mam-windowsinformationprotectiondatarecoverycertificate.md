---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: tfitzmac
ms.openlocfilehash: a66c1eeae6d405aa8d0546ac0143e2a8b3404231
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361661"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="8f3ef-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f3ef-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="8f3ef-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8f3ef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f3ef-105">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8f3ef-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="8f3ef-106">属性</span><span class="sxs-lookup"><span data-stu-id="8f3ef-106">Properties</span></span>
|<span data-ttu-id="8f3ef-107">属性</span><span class="sxs-lookup"><span data-stu-id="8f3ef-107">Property</span></span>|<span data-ttu-id="8f3ef-108">类型</span><span class="sxs-lookup"><span data-stu-id="8f3ef-108">Type</span></span>|<span data-ttu-id="8f3ef-109">说明</span><span class="sxs-lookup"><span data-stu-id="8f3ef-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f3ef-110">SubjectName</span><span class="sxs-lookup"><span data-stu-id="8f3ef-110">subjectName</span></span>|<span data-ttu-id="8f3ef-111">String</span><span class="sxs-lookup"><span data-stu-id="8f3ef-111">String</span></span>|<span data-ttu-id="8f3ef-112">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="8f3ef-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="8f3ef-113">description</span><span class="sxs-lookup"><span data-stu-id="8f3ef-113">description</span></span>|<span data-ttu-id="8f3ef-114">String</span><span class="sxs-lookup"><span data-stu-id="8f3ef-114">String</span></span>|<span data-ttu-id="8f3ef-115">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="8f3ef-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="8f3ef-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8f3ef-116">expirationDateTime</span></span>|<span data-ttu-id="8f3ef-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f3ef-117">DateTimeOffset</span></span>|<span data-ttu-id="8f3ef-118">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="8f3ef-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="8f3ef-119">证书</span><span class="sxs-lookup"><span data-stu-id="8f3ef-119">certificate</span></span>|<span data-ttu-id="8f3ef-120">Binary</span><span class="sxs-lookup"><span data-stu-id="8f3ef-120">Binary</span></span>|<span data-ttu-id="8f3ef-121">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="8f3ef-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f3ef-122">关系</span><span class="sxs-lookup"><span data-stu-id="8f3ef-122">Relationships</span></span>
<span data-ttu-id="8f3ef-123">无</span><span class="sxs-lookup"><span data-stu-id="8f3ef-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8f3ef-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f3ef-124">JSON Representation</span></span>
<span data-ttu-id="8f3ef-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f3ef-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



