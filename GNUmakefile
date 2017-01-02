THISDIR := curvilinear
THISBOOK := $(THISDIR)
BASEVER := 0179e84

include ../latex/make.vars

FIGURES := ../../figures/$(THISBOOK)
SOURCE_DIRS += $(FIGURES)

GENERATED_PDFS += $(THISBOOK).pdf

all :: $(COPIED_FILES)
all :: myrefs.bib $(GENERATED_PDFS)

$(THISBOOK).pdf :: $(wildcard *.tex)
$(GENERATED_PDFS) :: $(JUSTBOOKDEPENDENCIES) $(LOCAL_FILES) $(GENERATED_SOURCES) $(COPIED_FILES) $(LOCAL_COPIED_FILES)

include ../latex/make.rules
