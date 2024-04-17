
from pins import board_folder
from vetiver import VetiverAPI
from vetiver import VetiverModel

model_board = board_folder(
  "~/data/model", 
  allow_pickle_read = True
)

v = VetiverModel.from_pin(model_board, 'penguin_weight_predictor')#, version = '20240415T150347Z-8d7d5')

app = VetiverAPI(v, check_prototype = True)

app.run(port = 8082)
