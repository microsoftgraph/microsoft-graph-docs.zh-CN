---
title: Windows更新 API 概述
description: 适用于Windows更新部署服务可让你的组织控制提供给你的设备的更新。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: df2977584ba523f6efcc71366bd63db481539ce1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117625"
---
# <a name="windows-updates-api-overview"></a>Windows更新 API 概述

The Windows Update for Business deployment service provides control over device updates through the ability to approve， schedule and safeguard content delivered by Windows Update. 

## <a name="why-use-the-windows-update-for-business-deployment-service"></a>为什么使用 Windows Update for Business 部署服务？

IT 专业人员和管理工具供应商都可以使用部署服务：
* 将更新部署安排在特定的日期开始
* 使用富表达式在几天或几周内阶段部署
* 绕过预配置的 Windows Update for Business 策略以立即部署安全更新
* 通过针对唯一设备填充和移动设备配置定制的部署，确保 (硬件和软件) 

如今，部署服务支持管理Windows 10功能更新和Windows 10安全更新。 若要了解有关企业更新上下文中部署服务Windows，请参阅[部署服务概述](https://docs.microsoft.com/windows/deployment/update/deployment-service-overview)。

## <a name="prerequisites"></a>先决条件    

若要使用部署服务，组织必须拥有以下订阅之一：
* Windows 10 企业版E3 或 E5 (包含在 Microsoft 365 F3、E3 或 E5) 
* Windows 10 教育版A3 或 A5 (包含在 Microsoft 365 A3 或 A5) 
* Windows虚拟桌面访问 E3 或 E5
* Microsoft 365 商业高级版

此外，部署服务管理的设备必须：
* 加入 Azure AD 或加入混合 AD
* 运行下列版本之Windows 10：Windows 10 专业版、Windows 10 企业版、Windows 10 教育版、Windows 10 专业教育版
* 已安装Windows 10版本 1709 或更高版本

## <a name="enroll-devices-to-be-managed"></a>注册要管理的设备

若要开始使用部署服务， [请注册更新管理中的设备](windowsupdates-enroll.md)。

## <a name="approve-and-schedule-windows-content-delivered-from-windows-update"></a>批准和安排Windows更新中Windows的内容

部署服务简化了针对各种设备生态系统的审阅、批准、计划和部署内容。 存在更新目录以提供专为审批定制的视图，帮助您重点关注重要的审批决策，并避免需要对相关更新的深入列表进行排序。

选择要部署的更新后，可以计划部署以在将来开始，或部署一段时间。 如果选择在一段时间内部署更新，部署服务将自动优化设备提供更新的顺序。 如果可能，该服务对设备进行订购，以确保在部署早期表示硬件和软件资产的多样性，以最大限度地减少可能遇到意外更新问题的设备数量。 

详细了解部署服务：
* [软件更新](windowsupdates-software-updates.md)
* [部署](windowsupdates-deployments.md)
* [安排部署](windowsupdates-schedule-deployment.md)

## <a name="immediately-deploy-an-update-when-critical-needs-arise"></a>出现关键需求时立即部署更新

在出现关键安全问题的情况下，可以使用部署服务绕过标准更新策略并加快安全更新的部署。

若要了解更多信息，请参阅 [部署加速安全更新](windowsupdates-deploy-expedited-update.md)。

## <a name="protect-devices-by-default"></a>默认情况下保护设备

享受保护 [保留的好处](https://docs.microsoft.com/windows/deployment/update/safeguard-holds) ，防止出现质量或兼容性问题的设备安装更新，否则导致失败或回滚。

此外，还可以配置组织独有的监视规则。 这些规则可以基于设备信号（如回滚）发送警报或暂停部署。

若要了解更多信息，请参阅 [管理部署的监视规则](windowsupdates-manage-monitoring-rules.md)。

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

请参阅[microsoft Windows beta 中的 Graph 更新 API。](/graph/api/resources/windowsupdates-updates?view=graph-rest-beta&preserve-view=true)
