---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
ms.openlocfilehash: 68faf0e78c68468216c3e69d64926f2c8b18e3c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010239"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="3cc61-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="3cc61-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="3cc61-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3cc61-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cc61-105">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="3cc61-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="3cc61-106">属性</span><span class="sxs-lookup"><span data-stu-id="3cc61-106">Properties</span></span>
|<span data-ttu-id="3cc61-107">属性</span><span class="sxs-lookup"><span data-stu-id="3cc61-107">Property</span></span>|<span data-ttu-id="3cc61-108">类型</span><span class="sxs-lookup"><span data-stu-id="3cc61-108">Type</span></span>|<span data-ttu-id="3cc61-109">说明</span><span class="sxs-lookup"><span data-stu-id="3cc61-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cc61-110">SubjectName</span><span class="sxs-lookup"><span data-stu-id="3cc61-110">subjectName</span></span>|<span data-ttu-id="3cc61-111">String</span><span class="sxs-lookup"><span data-stu-id="3cc61-111">String</span></span>|<span data-ttu-id="3cc61-112">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="3cc61-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="3cc61-113">description</span><span class="sxs-lookup"><span data-stu-id="3cc61-113">description</span></span>|<span data-ttu-id="3cc61-114">String</span><span class="sxs-lookup"><span data-stu-id="3cc61-114">String</span></span>|<span data-ttu-id="3cc61-115">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="3cc61-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="3cc61-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3cc61-116">expirationDateTime</span></span>|<span data-ttu-id="3cc61-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cc61-117">DateTimeOffset</span></span>|<span data-ttu-id="3cc61-118">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="3cc61-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="3cc61-119">证书</span><span class="sxs-lookup"><span data-stu-id="3cc61-119">certificate</span></span>|<span data-ttu-id="3cc61-120">Binary</span><span class="sxs-lookup"><span data-stu-id="3cc61-120">Binary</span></span>|<span data-ttu-id="3cc61-121">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="3cc61-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cc61-122">关系</span><span class="sxs-lookup"><span data-stu-id="3cc61-122">Relationships</span></span>
<span data-ttu-id="3cc61-123">无</span><span class="sxs-lookup"><span data-stu-id="3cc61-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3cc61-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3cc61-124">JSON Representation</span></span>
<span data-ttu-id="3cc61-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3cc61-125">Here is a JSON representation of the resource.</span></span>
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



