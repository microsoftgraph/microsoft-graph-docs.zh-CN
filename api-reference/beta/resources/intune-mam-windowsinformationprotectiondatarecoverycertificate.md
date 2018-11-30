---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
ms.openlocfilehash: bbc6ae8e4607e5992ac9dd23fa1eb67e51d1ecd4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043123"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="b3dae-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3dae-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="b3dae-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b3dae-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3dae-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b3dae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3dae-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b3dae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3dae-107">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="b3dae-107">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="b3dae-108">属性</span><span class="sxs-lookup"><span data-stu-id="b3dae-108">Properties</span></span>
|<span data-ttu-id="b3dae-109">属性</span><span class="sxs-lookup"><span data-stu-id="b3dae-109">Property</span></span>|<span data-ttu-id="b3dae-110">类型</span><span class="sxs-lookup"><span data-stu-id="b3dae-110">Type</span></span>|<span data-ttu-id="b3dae-111">说明</span><span class="sxs-lookup"><span data-stu-id="b3dae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3dae-112">SubjectName</span><span class="sxs-lookup"><span data-stu-id="b3dae-112">subjectName</span></span>|<span data-ttu-id="b3dae-113">String</span><span class="sxs-lookup"><span data-stu-id="b3dae-113">String</span></span>|<span data-ttu-id="b3dae-114">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="b3dae-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="b3dae-115">description</span><span class="sxs-lookup"><span data-stu-id="b3dae-115">description</span></span>|<span data-ttu-id="b3dae-116">String</span><span class="sxs-lookup"><span data-stu-id="b3dae-116">String</span></span>|<span data-ttu-id="b3dae-117">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="b3dae-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="b3dae-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b3dae-118">expirationDateTime</span></span>|<span data-ttu-id="b3dae-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3dae-119">DateTimeOffset</span></span>|<span data-ttu-id="b3dae-120">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="b3dae-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="b3dae-121">证书</span><span class="sxs-lookup"><span data-stu-id="b3dae-121">certificate</span></span>|<span data-ttu-id="b3dae-122">Binary</span><span class="sxs-lookup"><span data-stu-id="b3dae-122">Binary</span></span>|<span data-ttu-id="b3dae-123">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="b3dae-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3dae-124">关系</span><span class="sxs-lookup"><span data-stu-id="b3dae-124">Relationships</span></span>
<span data-ttu-id="b3dae-125">无</span><span class="sxs-lookup"><span data-stu-id="b3dae-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3dae-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3dae-126">JSON Representation</span></span>
<span data-ttu-id="b3dae-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3dae-127">Here is a JSON representation of the resource.</span></span>
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





